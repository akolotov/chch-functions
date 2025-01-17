const API_ENDPOINT = 'https://api.crhoy.net/ultimas/2025-01-10.json?v=3';

export default async (request, context) => {
  try {
    const response = await fetch(API_ENDPOINT);
    const data = await response.json();
    return Response.json({ data });
  } catch (error) {
    console.log(error);
    return Response.json({ error: 'Failed fetching data' }, { status: 500 });
  }
};
